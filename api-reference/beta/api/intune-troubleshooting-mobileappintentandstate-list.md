---
title: Lista mobileAppIntentAndStates
description: Lista as propriedades e os relacionamentos dos objetos mobileAppIntentAndState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 95fd038a37b81168fd0381d44bbdb2a29d604d0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841444"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="9ca58-103">Lista mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="9ca58-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="9ca58-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ca58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ca58-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ca58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ca58-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ca58-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ca58-107">Lista as propriedades e os relacionamentos dos objetos [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="9ca58-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ca58-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ca58-108">Prerequisites</span></span>
<span data-ttu-id="9ca58-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ca58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ca58-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ca58-111">Permission type</span></span>|<span data-ttu-id="9ca58-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ca58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ca58-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ca58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ca58-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ca58-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9ca58-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ca58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ca58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ca58-116">Not supported.</span></span>|
|<span data-ttu-id="9ca58-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ca58-117">Application</span></span>|<span data-ttu-id="9ca58-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ca58-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ca58-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ca58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="9ca58-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca58-120">Request headers</span></span>
|<span data-ttu-id="9ca58-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ca58-121">Header</span></span>|<span data-ttu-id="9ca58-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ca58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ca58-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ca58-123">Authorization</span></span>|<span data-ttu-id="9ca58-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ca58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ca58-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ca58-125">Accept</span></span>|<span data-ttu-id="9ca58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ca58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ca58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca58-127">Request body</span></span>
<span data-ttu-id="9ca58-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ca58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ca58-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca58-129">Response</span></span>
<span data-ttu-id="9ca58-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ca58-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ca58-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ca58-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ca58-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca58-132">Request</span></span>
<span data-ttu-id="9ca58-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ca58-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="9ca58-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca58-134">Response</span></span>
<span data-ttu-id="9ca58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ca58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```





