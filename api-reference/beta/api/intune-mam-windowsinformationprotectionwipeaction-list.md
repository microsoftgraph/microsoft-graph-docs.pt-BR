---
title: Listar windowsInformationProtectionWipeActions
description: Listar Propriedades e relações dos objetos windowsInformationProtectionWipeAction.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99ffffba71de95d0bec7aed2f8f3448f0cc1045b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981500"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="10dbf-103">Listar windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="10dbf-103">List windowsInformationProtectionWipeActions</span></span>

> <span data-ttu-id="10dbf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10dbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10dbf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10dbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10dbf-106">Listar Propriedades e relações dos objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="10dbf-106">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10dbf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10dbf-107">Prerequisites</span></span>
<span data-ttu-id="10dbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10dbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10dbf-110">Permission type</span></span>|<span data-ttu-id="10dbf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10dbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10dbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10dbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10dbf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10dbf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10dbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10dbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10dbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10dbf-115">Not supported.</span></span>|
|<span data-ttu-id="10dbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10dbf-116">Application</span></span>|<span data-ttu-id="10dbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10dbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10dbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10dbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="10dbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10dbf-119">Request headers</span></span>
|<span data-ttu-id="10dbf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10dbf-120">Header</span></span>|<span data-ttu-id="10dbf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10dbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10dbf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10dbf-122">Authorization</span></span>|<span data-ttu-id="10dbf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10dbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10dbf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10dbf-124">Accept</span></span>|<span data-ttu-id="10dbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10dbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10dbf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10dbf-126">Request body</span></span>
<span data-ttu-id="10dbf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10dbf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10dbf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="10dbf-128">Response</span></span>
<span data-ttu-id="10dbf-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10dbf-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10dbf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10dbf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="10dbf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10dbf-131">Request</span></span>
<span data-ttu-id="10dbf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10dbf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="10dbf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="10dbf-133">Response</span></span>
<span data-ttu-id="10dbf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10dbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





