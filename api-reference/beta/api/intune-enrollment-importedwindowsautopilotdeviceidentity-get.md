---
title: Obter importedWindowsAutopilotDeviceIdentity
description: Lê as propriedades e relações do objeto importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccd930a0412968e18870333349fd1c5704ef7635
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159036"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="c0e88-103">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c0e88-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="c0e88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0e88-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0e88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0e88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0e88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e88-107">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="c0e88-107">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0e88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0e88-108">Prerequisites</span></span>
<span data-ttu-id="c0e88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0e88-111">Permission type</span></span>|<span data-ttu-id="c0e88-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0e88-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e88-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0e88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e88-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0e88-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0e88-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0e88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0e88-116">Not supported.</span></span>|
|<span data-ttu-id="c0e88-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0e88-117">Application</span></span>|<span data-ttu-id="c0e88-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0e88-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e88-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0e88-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0e88-120">Optional query parameters</span></span>
<span data-ttu-id="c0e88-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e88-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0e88-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e88-122">Request headers</span></span>
|<span data-ttu-id="c0e88-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0e88-123">Header</span></span>|<span data-ttu-id="c0e88-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c0e88-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e88-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0e88-125">Authorization</span></span>|<span data-ttu-id="c0e88-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0e88-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e88-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0e88-127">Accept</span></span>|<span data-ttu-id="c0e88-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e88-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e88-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e88-129">Request body</span></span>
<span data-ttu-id="c0e88-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0e88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e88-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e88-131">Response</span></span>
<span data-ttu-id="c0e88-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e88-132">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e88-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0e88-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0e88-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e88-134">Request</span></span>
<span data-ttu-id="c0e88-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0e88-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="c0e88-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e88-136">Response</span></span>
<span data-ttu-id="c0e88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0e88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "groupTag": "Group Tag value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "importId": "Import Id value",
    "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
    "state": {
      "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
      "deviceImportStatus": "pending",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceErrorCode": 15,
      "deviceErrorName": "Device Error Name value"
    },
    "assignedUserPrincipalName": "Assigned User Principal Name value"
  }
}
```




