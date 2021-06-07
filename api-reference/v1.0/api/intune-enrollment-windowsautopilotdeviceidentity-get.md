---
title: Obter windowsAutopilotDeviceIdentity
description: Ler propriedades e relações do objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8039791e1371d50cf38c69dd6026bfeffc7463e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752858"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="79cef-103">Obter windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="79cef-103">Get windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="79cef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79cef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79cef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79cef-106">Ler propriedades e relações do [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="79cef-106">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79cef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79cef-107">Prerequisites</span></span>
<span data-ttu-id="79cef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79cef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79cef-110">Permission type</span></span>|<span data-ttu-id="79cef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79cef-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79cef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79cef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79cef-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cef-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79cef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79cef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79cef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79cef-115">Not supported.</span></span>|
|<span data-ttu-id="79cef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79cef-116">Application</span></span>|<span data-ttu-id="79cef-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cef-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79cef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79cef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79cef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79cef-119">Optional query parameters</span></span>
<span data-ttu-id="79cef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79cef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79cef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79cef-121">Request headers</span></span>
|<span data-ttu-id="79cef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79cef-122">Header</span></span>|<span data-ttu-id="79cef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="79cef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79cef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="79cef-124">Authorization</span></span>|<span data-ttu-id="79cef-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79cef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79cef-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79cef-126">Accept</span></span>|<span data-ttu-id="79cef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79cef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79cef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79cef-128">Request body</span></span>
<span data-ttu-id="79cef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79cef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79cef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="79cef-130">Response</span></span>
<span data-ttu-id="79cef-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79cef-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79cef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79cef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="79cef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79cef-133">Request</span></span>
<span data-ttu-id="79cef-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79cef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="79cef-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="79cef-135">Response</span></span>
<span data-ttu-id="79cef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79cef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
    "groupTag": "Group Tag value",
    "purchaseOrderIdentifier": "Purchase Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "enrollmentState": "enrolled",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "addressableUserName": "Addressable User Name value",
    "userPrincipalName": "User Principal Name value",
    "resourceName": "Resource Name value",
    "skuNumber": "Sku Number value",
    "systemFamily": "System Family value",
    "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
    "managedDeviceId": "Managed Device Id value",
    "displayName": "Display Name value"
  }
}
```




