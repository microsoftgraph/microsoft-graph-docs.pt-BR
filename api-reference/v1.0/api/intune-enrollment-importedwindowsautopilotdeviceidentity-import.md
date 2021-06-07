---
title: ação de importação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 750b525ec0cdf7c28213787920c8164f7fcb1ac5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752869"
---
# <a name="import-action"></a><span data-ttu-id="9957c-103">ação de importação</span><span class="sxs-lookup"><span data-stu-id="9957c-103">import action</span></span>

<span data-ttu-id="9957c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9957c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9957c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9957c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9957c-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9957c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9957c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9957c-107">Prerequisites</span></span>
<span data-ttu-id="9957c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9957c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9957c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9957c-110">Permission type</span></span>|<span data-ttu-id="9957c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9957c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9957c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9957c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9957c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9957c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9957c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9957c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9957c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9957c-115">Not supported.</span></span>|
|<span data-ttu-id="9957c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9957c-116">Application</span></span>|<span data-ttu-id="9957c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9957c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9957c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9957c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="9957c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9957c-119">Request headers</span></span>
|<span data-ttu-id="9957c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9957c-120">Header</span></span>|<span data-ttu-id="9957c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9957c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9957c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9957c-122">Authorization</span></span>|<span data-ttu-id="9957c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9957c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9957c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9957c-124">Accept</span></span>|<span data-ttu-id="9957c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9957c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9957c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9957c-126">Request body</span></span>
<span data-ttu-id="9957c-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9957c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9957c-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9957c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9957c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9957c-129">Property</span></span>|<span data-ttu-id="9957c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9957c-130">Type</span></span>|<span data-ttu-id="9957c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9957c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9957c-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="9957c-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="9957c-133">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9957c-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="9957c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9957c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9957c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9957c-135">Response</span></span>
<span data-ttu-id="9957c-136">Se tiver êxito, essa ação retornará um código de resposta e uma `200 OK` [coleção importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9957c-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9957c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9957c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9957c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9957c-138">Request</span></span>
<span data-ttu-id="9957c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9957c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 808

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="9957c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9957c-140">Response</span></span>
<span data-ttu-id="9957c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9957c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 773

{
  "value": [
    {
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
  ]
}
```




