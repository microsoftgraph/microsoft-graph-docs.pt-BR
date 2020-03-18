---
title: Listar windowsInformationProtectionWipeActions
description: Listar Propriedades e relações dos objetos windowsInformationProtectionWipeAction.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2060d58e5beb2dd548670f5d5903549cd12028d5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803200"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="2ab98-103">Listar windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="2ab98-103">List windowsInformationProtectionWipeActions</span></span>

> <span data-ttu-id="2ab98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ab98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ab98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab98-106">Listar Propriedades e relações dos objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab98-106">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ab98-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ab98-107">Prerequisites</span></span>
<span data-ttu-id="2ab98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab98-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ab98-110">Permission type</span></span>|<span data-ttu-id="2ab98-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ab98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab98-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ab98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab98-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab98-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ab98-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ab98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ab98-115">Not supported.</span></span>|
|<span data-ttu-id="2ab98-116">Application</span><span class="sxs-lookup"><span data-stu-id="2ab98-116">Application</span></span>|<span data-ttu-id="2ab98-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab98-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab98-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ab98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="2ab98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab98-119">Request headers</span></span>
|<span data-ttu-id="2ab98-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ab98-120">Header</span></span>|<span data-ttu-id="2ab98-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ab98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ab98-122">Authorization</span></span>|<span data-ttu-id="2ab98-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ab98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab98-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ab98-124">Accept</span></span>|<span data-ttu-id="2ab98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab98-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab98-126">Request body</span></span>
<span data-ttu-id="2ab98-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ab98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab98-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ab98-128">Response</span></span>
<span data-ttu-id="2ab98-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ab98-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab98-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ab98-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ab98-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab98-131">Request</span></span>
<span data-ttu-id="2ab98-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ab98-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="2ab98-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ab98-133">Response</span></span>
<span data-ttu-id="2ab98-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ab98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "2620a996-a996-2620-96a9-202696a92026",
      "status": "pending",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
    }
  ]
}
```




