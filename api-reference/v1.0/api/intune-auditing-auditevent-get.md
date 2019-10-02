---
title: Get auditEvent
description: Ler propriedades e relações do objeto auditEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b711362bd9aecf38c863157c97136776a868d33a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354858"
---
# <a name="get-auditevent"></a><span data-ttu-id="13613-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="13613-103">Get auditEvent</span></span>

> <span data-ttu-id="13613-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13613-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13613-105">Ler propriedades e relações do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="13613-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13613-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13613-106">Prerequisites</span></span>
<span data-ttu-id="13613-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13613-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13613-109">Permission type</span></span>|<span data-ttu-id="13613-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13613-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13613-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13613-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13613-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13613-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13613-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13613-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13613-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13613-114">Not supported.</span></span>|
|<span data-ttu-id="13613-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13613-115">Application</span></span>|<span data-ttu-id="13613-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13613-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13613-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13613-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13613-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13613-118">Optional query parameters</span></span>
<span data-ttu-id="13613-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13613-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13613-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13613-120">Request headers</span></span>
|<span data-ttu-id="13613-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13613-121">Header</span></span>|<span data-ttu-id="13613-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13613-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13613-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13613-123">Authorization</span></span>|<span data-ttu-id="13613-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13613-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13613-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13613-125">Accept</span></span>|<span data-ttu-id="13613-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13613-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13613-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13613-127">Request body</span></span>
<span data-ttu-id="13613-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13613-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13613-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="13613-129">Response</span></span>
<span data-ttu-id="13613-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13613-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13613-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13613-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="13613-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13613-132">Request</span></span>
<span data-ttu-id="13613-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13613-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="13613-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="13613-134">Response</span></span>
<span data-ttu-id="13613-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13613-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
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
}
```




