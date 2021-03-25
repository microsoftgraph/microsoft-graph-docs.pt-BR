---
title: ação de importação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 179f1a62d49a08b0b61d81b13f19686f8f527c12
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159029"
---
# <a name="import-action"></a><span data-ttu-id="f771c-103">ação de importação</span><span class="sxs-lookup"><span data-stu-id="f771c-103">import action</span></span>

<span data-ttu-id="f771c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f771c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f771c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f771c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f771c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f771c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f771c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f771c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f771c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f771c-108">Prerequisites</span></span>
<span data-ttu-id="f771c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f771c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f771c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f771c-111">Permission type</span></span>|<span data-ttu-id="f771c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f771c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f771c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f771c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f771c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f771c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f771c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f771c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f771c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f771c-116">Not supported.</span></span>|
|<span data-ttu-id="f771c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f771c-117">Application</span></span>|<span data-ttu-id="f771c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f771c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f771c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f771c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="f771c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f771c-120">Request headers</span></span>
|<span data-ttu-id="f771c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f771c-121">Header</span></span>|<span data-ttu-id="f771c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f771c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f771c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f771c-123">Authorization</span></span>|<span data-ttu-id="f771c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f771c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f771c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f771c-125">Accept</span></span>|<span data-ttu-id="f771c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f771c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f771c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f771c-127">Request body</span></span>
<span data-ttu-id="f771c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f771c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f771c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f771c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f771c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f771c-130">Property</span></span>|<span data-ttu-id="f771c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f771c-131">Type</span></span>|<span data-ttu-id="f771c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f771c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f771c-133">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="f771c-133">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="f771c-134">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f771c-134">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="f771c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f771c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f771c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f771c-136">Response</span></span>
<span data-ttu-id="f771c-137">Se tiver êxito, essa ação retornará um código de resposta e uma `200 OK` [coleção importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f771c-137">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f771c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f771c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f771c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f771c-139">Request</span></span>
<span data-ttu-id="f771c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f771c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

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

### <a name="response"></a><span data-ttu-id="f771c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f771c-141">Response</span></span>
<span data-ttu-id="f771c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f771c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




