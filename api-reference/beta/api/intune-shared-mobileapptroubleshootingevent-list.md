---
title: Listar mobileAppTroubleshootingEvents
description: Descreve o método List mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04197f9a6364cbd25816d4f860c2d57d94360fee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458228"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="5978e-103">Listar mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="5978e-103">List mobileAppTroubleshootingEvents</span></span>

<span data-ttu-id="5978e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5978e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5978e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5978e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5978e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5978e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5978e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5978e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5978e-108">Listar Propriedades e relações dos objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="5978e-108">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5978e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5978e-109">Prerequisites</span></span>
<span data-ttu-id="5978e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5978e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5978e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5978e-112">Permission type</span></span>|<span data-ttu-id="5978e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5978e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5978e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5978e-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="5978e-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5978e-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="5978e-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5978e-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5978e-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="5978e-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="5978e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5978e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5978e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5978e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5978e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5978e-120">Not supported.</span></span>|
|<span data-ttu-id="5978e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5978e-121">Application</span></span>||
|<span data-ttu-id="5978e-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5978e-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="5978e-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5978e-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5978e-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="5978e-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="5978e-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5978e-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5978e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5978e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="5978e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5978e-127">Request headers</span></span>
|<span data-ttu-id="5978e-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5978e-128">Header</span></span>|<span data-ttu-id="5978e-129">Valor</span><span class="sxs-lookup"><span data-stu-id="5978e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5978e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5978e-130">Authorization</span></span>|<span data-ttu-id="5978e-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5978e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5978e-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5978e-132">Accept</span></span>|<span data-ttu-id="5978e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5978e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5978e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5978e-134">Request body</span></span>
<span data-ttu-id="5978e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5978e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5978e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5978e-136">Response</span></span>
<span data-ttu-id="5978e-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5978e-137">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5978e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5978e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5978e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5978e-139">Request</span></span>
<span data-ttu-id="5978e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5978e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="5978e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5978e-141">Response</span></span>
<span data-ttu-id="5978e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5978e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












