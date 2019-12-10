---
title: ação de importação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ad866ad8180a6e65d7dafe2628bcb9e9be2921b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943772"
---
# <a name="import-action"></a><span data-ttu-id="32184-103">ação de importação</span><span class="sxs-lookup"><span data-stu-id="32184-103">import action</span></span>

> <span data-ttu-id="32184-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32184-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32184-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32184-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32184-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32184-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32184-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32184-107">Prerequisites</span></span>
<span data-ttu-id="32184-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32184-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32184-110">Permission type</span></span>|<span data-ttu-id="32184-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32184-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32184-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32184-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32184-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32184-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32184-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32184-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32184-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32184-115">Not supported.</span></span>|
|<span data-ttu-id="32184-116">Application</span><span class="sxs-lookup"><span data-stu-id="32184-116">Application</span></span>|<span data-ttu-id="32184-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32184-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32184-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32184-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="32184-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32184-119">Request headers</span></span>
|<span data-ttu-id="32184-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32184-120">Header</span></span>|<span data-ttu-id="32184-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32184-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32184-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32184-122">Authorization</span></span>|<span data-ttu-id="32184-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32184-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32184-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32184-124">Accept</span></span>|<span data-ttu-id="32184-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32184-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32184-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32184-126">Request body</span></span>
<span data-ttu-id="32184-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="32184-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32184-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="32184-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32184-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32184-129">Property</span></span>|<span data-ttu-id="32184-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="32184-130">Type</span></span>|<span data-ttu-id="32184-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="32184-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32184-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="32184-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="32184-133">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="32184-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="32184-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32184-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32184-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32184-135">Response</span></span>
<span data-ttu-id="32184-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32184-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32184-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32184-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="32184-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32184-138">Request</span></span>
<span data-ttu-id="32184-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32184-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 860

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
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

### <a name="response"></a><span data-ttu-id="32184-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="32184-140">Response</span></span>
<span data-ttu-id="32184-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32184-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 825

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
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





