---
title: Lista windowsInformationProtectionWipeActions
description: Lista as propriedades e os relacionamentos dos objetos windowsInformationProtectionWipeAction.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07780e126239d808856e5a2e44e63cd75fc3747c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428999"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="dbbd2-103">Lista windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="dbbd2-103">List windowsInformationProtectionWipeActions</span></span>

> <span data-ttu-id="dbbd2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dbbd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbbd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbbd2-107">Lista as propriedades e os relacionamentos dos objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="dbbd2-107">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbbd2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbbd2-108">Prerequisites</span></span>
<span data-ttu-id="dbbd2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dbbd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dbbd2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbbd2-111">Permission type</span></span>|<span data-ttu-id="dbbd2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbbd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbbd2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbbd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbbd2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbd2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dbbd2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbbd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbbd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-116">Not supported.</span></span>|
|<span data-ttu-id="dbbd2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbbd2-117">Application</span></span>|<span data-ttu-id="dbbd2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbbd2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbbd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="dbbd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbbd2-120">Request headers</span></span>
|<span data-ttu-id="dbbd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbbd2-121">Header</span></span>|<span data-ttu-id="dbbd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dbbd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbbd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbbd2-123">Authorization</span></span>|<span data-ttu-id="dbbd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbbd2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbbd2-125">Accept</span></span>|<span data-ttu-id="dbbd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbbd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbbd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbbd2-127">Request body</span></span>
<span data-ttu-id="dbbd2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbbd2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbbd2-129">Response</span></span>
<span data-ttu-id="dbbd2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbbd2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbbd2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbbd2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbbd2-132">Request</span></span>
<span data-ttu-id="dbbd2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="dbbd2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbbd2-134">Response</span></span>
<span data-ttu-id="dbbd2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbbd2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "2620a996-a996-2620-96a9-202696a92026",
      "status": "pending",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value"
    }
  ]
}
```




