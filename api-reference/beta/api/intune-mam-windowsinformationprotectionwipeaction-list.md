---
title: Listar windowsInformationProtectionWipeActions
description: Listar Propriedades e relações dos objetos windowsInformationProtectionWipeAction.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc016087511b920fa9c420ce66efba072d0271d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529083"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="e0dca-103">Listar windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="e0dca-103">List windowsInformationProtectionWipeActions</span></span>

> <span data-ttu-id="e0dca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0dca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0dca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0dca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0dca-106">Listar Propriedades e relações dos objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="e0dca-106">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0dca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0dca-107">Prerequisites</span></span>
<span data-ttu-id="e0dca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0dca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0dca-110">Permission type</span></span>|<span data-ttu-id="e0dca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0dca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0dca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0dca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0dca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0dca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e0dca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0dca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0dca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0dca-115">Not supported.</span></span>|
|<span data-ttu-id="e0dca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0dca-116">Application</span></span>|<span data-ttu-id="e0dca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0dca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0dca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0dca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="e0dca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dca-119">Request headers</span></span>
|<span data-ttu-id="e0dca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0dca-120">Header</span></span>|<span data-ttu-id="e0dca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e0dca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0dca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0dca-122">Authorization</span></span>|<span data-ttu-id="e0dca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0dca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0dca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0dca-124">Accept</span></span>|<span data-ttu-id="e0dca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0dca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0dca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dca-126">Request body</span></span>
<span data-ttu-id="e0dca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0dca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0dca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0dca-128">Response</span></span>
<span data-ttu-id="e0dca-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0dca-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0dca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0dca-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0dca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dca-131">Request</span></span>
<span data-ttu-id="e0dca-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0dca-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="e0dca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0dca-133">Response</span></span>
<span data-ttu-id="e0dca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0dca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





