---
title: Listar mobileAppTroubleshootingEvents
description: Descreve o método List mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e3f25d4116d2dcbb577be968bf880e785d498b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993561"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="a5e04-103">Listar mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="a5e04-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="a5e04-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5e04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5e04-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5e04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5e04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5e04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5e04-107">Listar Propriedades e relações dos objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a5e04-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5e04-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5e04-108">Prerequisites</span></span>
<span data-ttu-id="a5e04-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5e04-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e04-111">Permission type</span></span>|<span data-ttu-id="a5e04-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5e04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5e04-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e04-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="a5e04-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="a5e04-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="a5e04-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e04-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a5e04-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="a5e04-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="a5e04-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e04-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a5e04-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e04-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5e04-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e04-119">Not supported.</span></span>|
|<span data-ttu-id="a5e04-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e04-120">Application</span></span>|<span data-ttu-id="a5e04-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e04-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5e04-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e04-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a5e04-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e04-123">Request headers</span></span>
|<span data-ttu-id="a5e04-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5e04-124">Header</span></span>|<span data-ttu-id="a5e04-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a5e04-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5e04-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e04-126">Authorization</span></span>|<span data-ttu-id="a5e04-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e04-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5e04-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5e04-128">Accept</span></span>|<span data-ttu-id="a5e04-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a5e04-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5e04-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e04-130">Request body</span></span>
<span data-ttu-id="a5e04-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5e04-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5e04-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e04-132">Response</span></span>
<span data-ttu-id="a5e04-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e04-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e04-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e04-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5e04-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e04-135">Request</span></span>
<span data-ttu-id="a5e04-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e04-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="a5e04-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e04-137">Response</span></span>
<span data-ttu-id="a5e04-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




