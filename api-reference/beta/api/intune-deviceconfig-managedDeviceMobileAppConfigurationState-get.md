---
title: Obter managedDeviceMobileAppConfigurationState
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d83f3f1a011ad772f2b62914adb42a77c48ce87
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636039"
---
# <a name="get-manageddevicemobileappconfigurationstate"></a><span data-ttu-id="bba3a-103">Obter managedDeviceMobileAppConfigurationState</span><span class="sxs-lookup"><span data-stu-id="bba3a-103">Get managedDeviceMobileAppConfigurationState</span></span>

> <span data-ttu-id="bba3a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bba3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bba3a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bba3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba3a-106">Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationState.</span><span class="sxs-lookup"><span data-stu-id="bba3a-106">Read properties and relationships of the managedDeviceMobileAppConfigurationState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bba3a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bba3a-107">Prerequisites</span></span>
<span data-ttu-id="bba3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bba3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba3a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bba3a-110">Permission type</span></span>|<span data-ttu-id="bba3a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bba3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bba3a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bba3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bba3a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bba3a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bba3a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bba3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bba3a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bba3a-115">Not supported.</span></span>|
|<span data-ttu-id="bba3a-116">Application</span><span class="sxs-lookup"><span data-stu-id="bba3a-116">Application</span></span>|<span data-ttu-id="bba3a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bba3a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bba3a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bba3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bba3a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bba3a-119">Optional query parameters</span></span>
<span data-ttu-id="bba3a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bba3a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bba3a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bba3a-121">Request headers</span></span>
|<span data-ttu-id="bba3a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bba3a-122">Header</span></span>|<span data-ttu-id="bba3a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bba3a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bba3a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bba3a-124">Authorization</span></span>|<span data-ttu-id="bba3a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bba3a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bba3a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bba3a-126">Accept</span></span>|<span data-ttu-id="bba3a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bba3a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bba3a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bba3a-128">Request body</span></span>
<span data-ttu-id="bba3a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bba3a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bba3a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bba3a-130">Response</span></span>
<span data-ttu-id="bba3a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto managedDeviceMobileAppConfigurationState no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bba3a-131">If successful, this method returns a `200 OK` response code and managedDeviceMobileAppConfigurationState object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bba3a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bba3a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bba3a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bba3a-133">Request</span></span>
<span data-ttu-id="bba3a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bba3a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

### <a name="response"></a><span data-ttu-id="bba3a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bba3a-135">Response</span></span>
<span data-ttu-id="bba3a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bba3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1225

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
    "id": "659554f2-54f2-6595-f254-9565f2549565",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
        "setting": "Setting value",
        "settingName": "Setting Name value",
        "instanceDisplayName": "Instance Display Name value",
        "state": "notApplicable",
        "errorCode": 9,
        "errorDescription": "Error Description value",
        "userId": "User Id value",
        "userName": "User Name value",
        "userEmail": "User Email value",
        "userPrincipalName": "User Principal Name value",
        "sources": [
          {
            "@odata.type": "microsoft.graph.settingSource",
            "id": "Id value",
            "displayName": "Display Name value"
          }
        ],
        "currentValue": "Current Value value"
      }
    ],
    "displayName": "Display Name value",
    "version": 7,
    "platformType": "androidForWork",
    "state": "notApplicable",
    "settingCount": 12,
    "userId": "User Id value",
    "userPrincipalName": "User Principal Name value"
  }
}
```



