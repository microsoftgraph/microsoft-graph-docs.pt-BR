---
title: Obter mobileAppTroubleshootingEvent
description: Descreve o método Get mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e940caa3da08c1879050a27af0872e03494b745f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800736"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="ae5d1-103">Obter mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ae5d1-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="ae5d1-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae5d1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae5d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae5d1-107">Leia as propriedades e as relações do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="ae5d1-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae5d1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae5d1-108">Prerequisites</span></span>
<span data-ttu-id="ae5d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae5d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae5d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae5d1-111">Permission type</span></span>|<span data-ttu-id="ae5d1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae5d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae5d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae5d1-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ae5d1-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae5d1-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ae5d1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae5d1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae5d1-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae5d1-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ae5d1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae5d1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae5d1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae5d1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae5d1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-119">Not supported.</span></span>|
|<span data-ttu-id="ae5d1-120">Application</span><span class="sxs-lookup"><span data-stu-id="ae5d1-120">Application</span></span>||
|<span data-ttu-id="ae5d1-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae5d1-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ae5d1-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae5d1-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae5d1-123">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae5d1-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ae5d1-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae5d1-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae5d1-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae5d1-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae5d1-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae5d1-126">Optional query parameters</span></span>
<span data-ttu-id="ae5d1-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae5d1-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae5d1-128">Request headers</span></span>
|<span data-ttu-id="ae5d1-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae5d1-129">Header</span></span>|<span data-ttu-id="ae5d1-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ae5d1-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae5d1-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae5d1-131">Authorization</span></span>|<span data-ttu-id="ae5d1-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae5d1-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae5d1-133">Accept</span></span>|<span data-ttu-id="ae5d1-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ae5d1-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae5d1-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae5d1-135">Request body</span></span>
<span data-ttu-id="ae5d1-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae5d1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae5d1-137">Response</span></span>
<span data-ttu-id="ae5d1-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-138">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae5d1-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae5d1-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae5d1-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae5d1-140">Request</span></span>
<span data-ttu-id="ae5d1-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ae5d1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae5d1-142">Response</span></span>
<span data-ttu-id="ae5d1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae5d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











