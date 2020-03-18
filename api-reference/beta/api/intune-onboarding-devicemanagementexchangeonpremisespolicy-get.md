---
title: Obter deviceManagementExchangeOnPremisesPolicy
description: Leia as propriedades e as relações do objeto deviceManagementExchangeOnPremisesPolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c81bbfb81d59e931f700b9a46999548a7eca9a37
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802892"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="a1539-103">Obter deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="a1539-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="a1539-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1539-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1539-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1539-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1539-106">Leia as propriedades e as relações do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a1539-106">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1539-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1539-107">Prerequisites</span></span>
<span data-ttu-id="a1539-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1539-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1539-110">Permission type</span></span>|<span data-ttu-id="a1539-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1539-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1539-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1539-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1539-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1539-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a1539-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1539-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1539-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1539-115">Not supported.</span></span>|
|<span data-ttu-id="a1539-116">Application</span><span class="sxs-lookup"><span data-stu-id="a1539-116">Application</span></span>|<span data-ttu-id="a1539-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1539-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1539-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1539-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1539-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1539-119">Optional query parameters</span></span>
<span data-ttu-id="a1539-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1539-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1539-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1539-121">Request headers</span></span>
|<span data-ttu-id="a1539-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1539-122">Header</span></span>|<span data-ttu-id="a1539-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a1539-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1539-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1539-124">Authorization</span></span>|<span data-ttu-id="a1539-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1539-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1539-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1539-126">Accept</span></span>|<span data-ttu-id="a1539-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1539-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1539-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1539-128">Request body</span></span>
<span data-ttu-id="a1539-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1539-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1539-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1539-130">Response</span></span>
<span data-ttu-id="a1539-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1539-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1539-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1539-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1539-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1539-133">Request</span></span>
<span data-ttu-id="a1539-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1539-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="a1539-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1539-135">Response</span></span>
<span data-ttu-id="a1539-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1539-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```




