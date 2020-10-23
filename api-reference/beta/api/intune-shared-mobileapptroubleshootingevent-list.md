---
title: Listar mobileAppTroubleshootingEvents
description: Descreve o método List mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23b0a109ac9154798178065489f6d2feb39eb3ae
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694239"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="3ae1b-103">Listar mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="3ae1b-103">List mobileAppTroubleshootingEvents</span></span>

<span data-ttu-id="3ae1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ae1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ae1b-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ae1b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ae1b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ae1b-108">Listar Propriedades e relações dos objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="3ae1b-108">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ae1b-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ae1b-109">Prerequisites</span></span>
<span data-ttu-id="3ae1b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ae1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ae1b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ae1b-112">Permission type</span></span>|<span data-ttu-id="3ae1b-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ae1b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ae1b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ae1b-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3ae1b-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3ae1b-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="3ae1b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae1b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3ae1b-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="3ae1b-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="3ae1b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae1b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3ae1b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ae1b-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ae1b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-120">Not supported.</span></span>|
|<span data-ttu-id="3ae1b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ae1b-121">Application</span></span>||
|<span data-ttu-id="3ae1b-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3ae1b-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="3ae1b-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae1b-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3ae1b-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="3ae1b-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="3ae1b-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae1b-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ae1b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ae1b-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="3ae1b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae1b-127">Request headers</span></span>
|<span data-ttu-id="3ae1b-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ae1b-128">Header</span></span>|<span data-ttu-id="3ae1b-129">Valor</span><span class="sxs-lookup"><span data-stu-id="3ae1b-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ae1b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ae1b-130">Authorization</span></span>|<span data-ttu-id="3ae1b-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ae1b-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ae1b-132">Accept</span></span>|<span data-ttu-id="3ae1b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3ae1b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ae1b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae1b-134">Request body</span></span>
<span data-ttu-id="3ae1b-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ae1b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae1b-136">Response</span></span>
<span data-ttu-id="3ae1b-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-137">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ae1b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ae1b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ae1b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae1b-139">Request</span></span>
<span data-ttu-id="3ae1b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="3ae1b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae1b-141">Response</span></span>
<span data-ttu-id="3ae1b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ae1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```












