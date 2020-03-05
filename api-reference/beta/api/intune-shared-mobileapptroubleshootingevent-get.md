---
title: Obter mobileAppTroubleshootingEvent
description: Descreve o método Get mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b366103d7dd2c2caf0e2b449e1f61d728268451b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458249"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="19ccc-103">Obter mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="19ccc-103">Get mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="19ccc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19ccc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19ccc-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19ccc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19ccc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19ccc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19ccc-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19ccc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ccc-108">Leia as propriedades e as relações do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="19ccc-108">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19ccc-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19ccc-109">Prerequisites</span></span>
<span data-ttu-id="19ccc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ccc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ccc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19ccc-112">Permission type</span></span>|<span data-ttu-id="19ccc-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19ccc-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19ccc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19ccc-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="19ccc-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="19ccc-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="19ccc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ccc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19ccc-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="19ccc-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="19ccc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ccc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19ccc-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19ccc-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19ccc-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19ccc-120">Not supported.</span></span>|
|<span data-ttu-id="19ccc-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19ccc-121">Application</span></span>||
|<span data-ttu-id="19ccc-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="19ccc-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="19ccc-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ccc-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19ccc-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="19ccc-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="19ccc-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ccc-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19ccc-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19ccc-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19ccc-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="19ccc-127">Optional query parameters</span></span>
<span data-ttu-id="19ccc-128">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="19ccc-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19ccc-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19ccc-129">Request headers</span></span>
|<span data-ttu-id="19ccc-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19ccc-130">Header</span></span>|<span data-ttu-id="19ccc-131">Valor</span><span class="sxs-lookup"><span data-stu-id="19ccc-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19ccc-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="19ccc-132">Authorization</span></span>|<span data-ttu-id="19ccc-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19ccc-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19ccc-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19ccc-134">Accept</span></span>|<span data-ttu-id="19ccc-135">application/json</span><span class="sxs-lookup"><span data-stu-id="19ccc-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ccc-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19ccc-136">Request body</span></span>
<span data-ttu-id="19ccc-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19ccc-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19ccc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="19ccc-138">Response</span></span>
<span data-ttu-id="19ccc-139">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19ccc-139">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ccc-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19ccc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="19ccc-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19ccc-141">Request</span></span>
<span data-ttu-id="19ccc-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19ccc-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="19ccc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="19ccc-143">Response</span></span>
<span data-ttu-id="19ccc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19ccc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477"
  }
}
```












