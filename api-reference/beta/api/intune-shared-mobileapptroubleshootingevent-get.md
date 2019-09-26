---
title: Obter mobileAppTroubleshootingEvent
description: Descreve o método Get mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12b1e6a8297d43bb34180b4fd28eb8009b3f4d12
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195941"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="16c43-103">Obter mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="16c43-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="16c43-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16c43-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16c43-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16c43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16c43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16c43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16c43-107">Leia as propriedades e as relações do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="16c43-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16c43-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16c43-108">Prerequisites</span></span>
<span data-ttu-id="16c43-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c43-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16c43-111">Permission type</span></span>|<span data-ttu-id="16c43-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16c43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16c43-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16c43-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="16c43-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="16c43-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="16c43-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c43-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="16c43-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="16c43-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="16c43-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c43-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="16c43-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16c43-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16c43-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16c43-119">Not supported.</span></span>|
|<span data-ttu-id="16c43-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16c43-120">Application</span></span>||
|<span data-ttu-id="16c43-121">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="16c43-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="16c43-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c43-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="16c43-123">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="16c43-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="16c43-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c43-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16c43-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16c43-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16c43-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16c43-126">Optional query parameters</span></span>
<span data-ttu-id="16c43-127">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16c43-127">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16c43-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16c43-128">Request headers</span></span>
|<span data-ttu-id="16c43-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16c43-129">Header</span></span>|<span data-ttu-id="16c43-130">Valor</span><span class="sxs-lookup"><span data-stu-id="16c43-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16c43-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="16c43-131">Authorization</span></span>|<span data-ttu-id="16c43-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16c43-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16c43-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16c43-133">Accept</span></span>|<span data-ttu-id="16c43-134">application/json</span><span class="sxs-lookup"><span data-stu-id="16c43-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16c43-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16c43-135">Request body</span></span>
<span data-ttu-id="16c43-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16c43-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16c43-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="16c43-137">Response</span></span>
<span data-ttu-id="16c43-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16c43-138">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16c43-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16c43-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="16c43-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16c43-140">Request</span></span>
<span data-ttu-id="16c43-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16c43-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="16c43-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="16c43-142">Response</span></span>
<span data-ttu-id="16c43-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16c43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








