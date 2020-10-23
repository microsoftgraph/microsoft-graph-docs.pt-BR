---
title: ação de importação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df7d1b6b069a66bd2f86a55a442aaa5f359517b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736433"
---
# <a name="import-action"></a><span data-ttu-id="fbaad-103">ação de importação</span><span class="sxs-lookup"><span data-stu-id="fbaad-103">import action</span></span>

<span data-ttu-id="fbaad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbaad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbaad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbaad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbaad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbaad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbaad-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fbaad-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbaad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbaad-108">Prerequisites</span></span>
<span data-ttu-id="fbaad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbaad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbaad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbaad-111">Permission type</span></span>|<span data-ttu-id="fbaad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbaad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbaad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbaad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbaad-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbaad-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbaad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbaad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbaad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbaad-116">Not supported.</span></span>|
|<span data-ttu-id="fbaad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbaad-117">Application</span></span>|<span data-ttu-id="fbaad-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbaad-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbaad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbaad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="fbaad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaad-120">Request headers</span></span>
|<span data-ttu-id="fbaad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbaad-121">Header</span></span>|<span data-ttu-id="fbaad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbaad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbaad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbaad-123">Authorization</span></span>|<span data-ttu-id="fbaad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbaad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbaad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbaad-125">Accept</span></span>|<span data-ttu-id="fbaad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbaad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbaad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaad-127">Request body</span></span>
<span data-ttu-id="fbaad-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fbaad-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fbaad-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fbaad-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fbaad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbaad-130">Property</span></span>|<span data-ttu-id="fbaad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbaad-131">Type</span></span>|<span data-ttu-id="fbaad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbaad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbaad-133">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="fbaad-133">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="fbaad-134">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fbaad-134">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="fbaad-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fbaad-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fbaad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaad-136">Response</span></span>
<span data-ttu-id="fbaad-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbaad-137">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbaad-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbaad-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbaad-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaad-139">Request</span></span>
<span data-ttu-id="fbaad-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbaad-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fbaad-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaad-141">Response</span></span>
<span data-ttu-id="fbaad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbaad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





