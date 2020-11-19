---
title: Listar windowsInformationProtectionWipeActions
description: Listar Propriedades e relações dos objetos windowsInformationProtectionWipeAction.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9ed778fb3978f9b5cf76a249b1e7198ad3b55ee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285629"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="04cb7-103">Listar windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="04cb7-103">List windowsInformationProtectionWipeActions</span></span>

<span data-ttu-id="04cb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04cb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04cb7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04cb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04cb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04cb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04cb7-107">Listar Propriedades e relações dos objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="04cb7-107">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04cb7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04cb7-108">Prerequisites</span></span>
<span data-ttu-id="04cb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04cb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04cb7-111">Permission type</span></span>|<span data-ttu-id="04cb7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04cb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04cb7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04cb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04cb7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04cb7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="04cb7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04cb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04cb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04cb7-116">Not supported.</span></span>|
|<span data-ttu-id="04cb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04cb7-117">Application</span></span>|<span data-ttu-id="04cb7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04cb7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04cb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04cb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="04cb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04cb7-120">Request headers</span></span>
|<span data-ttu-id="04cb7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04cb7-121">Header</span></span>|<span data-ttu-id="04cb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04cb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04cb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04cb7-123">Authorization</span></span>|<span data-ttu-id="04cb7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04cb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04cb7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04cb7-125">Accept</span></span>|<span data-ttu-id="04cb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04cb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04cb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04cb7-127">Request body</span></span>
<span data-ttu-id="04cb7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04cb7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04cb7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="04cb7-129">Response</span></span>
<span data-ttu-id="04cb7-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04cb7-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04cb7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04cb7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="04cb7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04cb7-132">Request</span></span>
<span data-ttu-id="04cb7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04cb7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="04cb7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="04cb7-134">Response</span></span>
<span data-ttu-id="04cb7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04cb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




