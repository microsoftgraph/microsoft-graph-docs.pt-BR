---
title: Obter mobileAppTroubleshootingEvent
description: Descreve o método de mobileAppTroubleshootingEvent Get da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6d151c28e909aecc1a0f20775d75813e0666df71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428949"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="f1549-103">Obter mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f1549-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="f1549-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1549-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1549-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1549-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1549-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f1549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1549-107">Leia as propriedades e os relacionamentos do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f1549-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1549-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1549-108">Prerequisites</span></span>
<span data-ttu-id="f1549-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1549-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1549-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1549-111">Permission type</span></span>|<span data-ttu-id="f1549-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1549-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1549-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1549-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f1549-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f1549-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f1549-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1549-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f1549-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="f1549-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f1549-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1549-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f1549-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1549-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1549-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1549-119">Not supported.</span></span>|
|<span data-ttu-id="f1549-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1549-120">Application</span></span>|<span data-ttu-id="f1549-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1549-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1549-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1549-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1549-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1549-123">Optional query parameters</span></span>
<span data-ttu-id="f1549-124">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1549-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1549-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1549-125">Request headers</span></span>
|<span data-ttu-id="f1549-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1549-126">Header</span></span>|<span data-ttu-id="f1549-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f1549-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1549-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1549-128">Authorization</span></span>|<span data-ttu-id="f1549-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1549-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1549-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1549-130">Accept</span></span>|<span data-ttu-id="f1549-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f1549-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1549-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1549-132">Request body</span></span>
<span data-ttu-id="f1549-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1549-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1549-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1549-134">Response</span></span>
<span data-ttu-id="f1549-135">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1549-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1549-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1549-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1549-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1549-137">Request</span></span>
<span data-ttu-id="f1549-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1549-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="f1549-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1549-139">Response</span></span>
<span data-ttu-id="f1549-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1549-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




