---
title: Obter deviceManagementExchangeOnPremisesPolicy
description: Leia as propriedades e os relacionamentos do objeto deviceManagementExchangeOnPremisesPolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a587e369fc99f1f6b3a0ec7478271e1669a19aba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832939"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="d2e09-103">Obter deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="d2e09-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="d2e09-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2e09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2e09-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2e09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2e09-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d2e09-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2e09-107">Leia as propriedades e os relacionamentos do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d2e09-107">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2e09-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2e09-108">Prerequisites</span></span>
<span data-ttu-id="d2e09-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2e09-111">Permission type</span></span>|<span data-ttu-id="d2e09-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2e09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2e09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2e09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2e09-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2e09-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d2e09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2e09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2e09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2e09-116">Not supported.</span></span>|
|<span data-ttu-id="d2e09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2e09-117">Application</span></span>|<span data-ttu-id="d2e09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2e09-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2e09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2e09-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2e09-120">Optional query parameters</span></span>
<span data-ttu-id="d2e09-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2e09-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d2e09-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e09-122">Request headers</span></span>
|<span data-ttu-id="d2e09-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2e09-123">Header</span></span>|<span data-ttu-id="d2e09-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d2e09-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2e09-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2e09-125">Authorization</span></span>|<span data-ttu-id="d2e09-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2e09-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2e09-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2e09-127">Accept</span></span>|<span data-ttu-id="d2e09-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d2e09-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2e09-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e09-129">Request body</span></span>
<span data-ttu-id="d2e09-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2e09-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2e09-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e09-131">Response</span></span>
<span data-ttu-id="d2e09-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2e09-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e09-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2e09-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2e09-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e09-134">Request</span></span>
<span data-ttu-id="d2e09-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2e09-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="d2e09-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e09-136">Response</span></span>
<span data-ttu-id="d2e09-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2e09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





