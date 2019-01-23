---
title: Lista mobileAppTroubleshootingEvents
description: Descreve o método mobileAppTroubleshootingEvent de lista da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79f89fd755b52bc0d9a3a1a1d0e0c6dc91853e76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429114"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="b6095-103">Lista mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="b6095-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="b6095-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6095-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6095-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6095-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6095-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b6095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6095-107">Lista as propriedades e os relacionamentos dos objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="b6095-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6095-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6095-108">Prerequisites</span></span>
<span data-ttu-id="b6095-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6095-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6095-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6095-111">Permission type</span></span>|<span data-ttu-id="b6095-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6095-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6095-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6095-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="b6095-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b6095-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="b6095-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6095-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b6095-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b6095-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="b6095-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6095-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b6095-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6095-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6095-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6095-119">Not supported.</span></span>|
|<span data-ttu-id="b6095-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6095-120">Application</span></span>|<span data-ttu-id="b6095-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6095-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6095-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6095-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b6095-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6095-123">Request headers</span></span>
|<span data-ttu-id="b6095-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6095-124">Header</span></span>|<span data-ttu-id="b6095-125">Valor</span><span class="sxs-lookup"><span data-stu-id="b6095-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6095-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6095-126">Authorization</span></span>|<span data-ttu-id="b6095-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6095-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6095-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6095-128">Accept</span></span>|<span data-ttu-id="b6095-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b6095-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6095-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6095-130">Request body</span></span>
<span data-ttu-id="b6095-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6095-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6095-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6095-132">Response</span></span>
<span data-ttu-id="b6095-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6095-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6095-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6095-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6095-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6095-135">Request</span></span>
<span data-ttu-id="b6095-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6095-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="b6095-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6095-137">Response</span></span>
<span data-ttu-id="b6095-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6095-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




