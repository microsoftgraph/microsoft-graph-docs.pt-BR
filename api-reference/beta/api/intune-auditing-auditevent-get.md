---
title: Get auditEvent
description: Ler propriedades e relações do objeto auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dae4e912ad18914b296d82920a2d3cbc2b1b98ee
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133231"
---
# <a name="get-auditevent"></a><span data-ttu-id="652f5-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="652f5-103">Get auditEvent</span></span>

<span data-ttu-id="652f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="652f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="652f5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="652f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="652f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="652f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652f5-107">Ler propriedades e relações do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="652f5-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="652f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="652f5-108">Prerequisites</span></span>
<span data-ttu-id="652f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="652f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="652f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="652f5-111">Permission type</span></span>|<span data-ttu-id="652f5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="652f5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="652f5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="652f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="652f5-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652f5-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="652f5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="652f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="652f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="652f5-116">Not supported.</span></span>|
|<span data-ttu-id="652f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="652f5-117">Application</span></span>|<span data-ttu-id="652f5-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652f5-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="652f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="652f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="652f5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="652f5-120">Optional query parameters</span></span>
<span data-ttu-id="652f5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="652f5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="652f5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="652f5-122">Request headers</span></span>
|<span data-ttu-id="652f5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="652f5-123">Header</span></span>|<span data-ttu-id="652f5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="652f5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="652f5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="652f5-125">Authorization</span></span>|<span data-ttu-id="652f5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="652f5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="652f5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="652f5-127">Accept</span></span>|<span data-ttu-id="652f5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="652f5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="652f5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="652f5-129">Request body</span></span>
<span data-ttu-id="652f5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="652f5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="652f5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="652f5-131">Response</span></span>
<span data-ttu-id="652f5-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="652f5-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="652f5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="652f5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="652f5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="652f5-134">Request</span></span>
<span data-ttu-id="652f5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="652f5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="652f5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="652f5-136">Response</span></span>
<span data-ttu-id="652f5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="652f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1863

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
}
```




