---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método Create mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33336696744e8878ec5324026c88671b4b71fe17
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537962"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="ab43d-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ab43d-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="ab43d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab43d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab43d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab43d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab43d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab43d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab43d-107">Criar um novo objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="ab43d-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab43d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab43d-108">Prerequisites</span></span>
<span data-ttu-id="ab43d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab43d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab43d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab43d-111">Permission type</span></span>|<span data-ttu-id="ab43d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab43d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab43d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab43d-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ab43d-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="ab43d-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ab43d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab43d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab43d-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="ab43d-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ab43d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab43d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab43d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab43d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab43d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab43d-119">Not supported.</span></span>|
|<span data-ttu-id="ab43d-120">Application</span><span class="sxs-lookup"><span data-stu-id="ab43d-120">Application</span></span>||
|<span data-ttu-id="ab43d-121">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="ab43d-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ab43d-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab43d-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab43d-123">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="ab43d-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ab43d-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab43d-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab43d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab43d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ab43d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab43d-126">Request headers</span></span>
|<span data-ttu-id="ab43d-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab43d-127">Header</span></span>|<span data-ttu-id="ab43d-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ab43d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab43d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab43d-129">Authorization</span></span>|<span data-ttu-id="ab43d-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab43d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab43d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab43d-131">Accept</span></span>|<span data-ttu-id="ab43d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="ab43d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab43d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab43d-133">Request body</span></span>
<span data-ttu-id="ab43d-134">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="ab43d-134">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="ab43d-135">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="ab43d-135">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="ab43d-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab43d-136">Property</span></span>|<span data-ttu-id="ab43d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab43d-137">Type</span></span>|<span data-ttu-id="ab43d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab43d-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab43d-139">id</span><span class="sxs-lookup"><span data-stu-id="ab43d-139">id</span></span>|<span data-ttu-id="ab43d-140">String</span><span class="sxs-lookup"><span data-stu-id="ab43d-140">String</span></span>|<span data-ttu-id="ab43d-141">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ab43d-141">The GUID for the object</span></span>|
|<span data-ttu-id="ab43d-142">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ab43d-142">**Troubleshooting**</span></span>|
|<span data-ttu-id="ab43d-143">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="ab43d-143">additionalInformation</span></span>|<span data-ttu-id="ab43d-144">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ab43d-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ab43d-145">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="ab43d-145">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="ab43d-146">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="ab43d-146">applicationId</span></span>|<span data-ttu-id="ab43d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab43d-147">String</span></span>|<span data-ttu-id="ab43d-148">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="ab43d-148">Intune application identifier.</span></span>|
|<span data-ttu-id="ab43d-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="ab43d-149">correlationId</span></span>|<span data-ttu-id="ab43d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab43d-150">String</span></span>|<span data-ttu-id="ab43d-151">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="ab43d-151">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="ab43d-152">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ab43d-152">eventDateTime</span></span>|<span data-ttu-id="ab43d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab43d-153">DateTimeOffset</span></span>|<span data-ttu-id="ab43d-154">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ab43d-154">Time when the event occurred .</span></span> |
|<span data-ttu-id="ab43d-155">EventName</span><span class="sxs-lookup"><span data-stu-id="ab43d-155">eventName</span></span>|<span data-ttu-id="ab43d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab43d-156">String</span></span>|<span data-ttu-id="ab43d-157">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="ab43d-157">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="ab43d-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab43d-158">Optional.</span></span>|
|<span data-ttu-id="ab43d-159">histórico</span><span class="sxs-lookup"><span data-stu-id="ab43d-159">history</span></span>|<span data-ttu-id="ab43d-160">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ab43d-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="ab43d-161">Item do histórico de solução de problemas do aplicativo móvel do Intune</span><span class="sxs-lookup"><span data-stu-id="ab43d-161">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="ab43d-162">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ab43d-162">managedDeviceIdentifier</span></span>|<span data-ttu-id="ab43d-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab43d-163">String</span></span>|<span data-ttu-id="ab43d-164">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="ab43d-164">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="ab43d-165">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab43d-165">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="ab43d-166">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab43d-166">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="ab43d-167">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="ab43d-167">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="ab43d-168">userId</span><span class="sxs-lookup"><span data-stu-id="ab43d-168">userId</span></span>|<span data-ttu-id="ab43d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab43d-169">String</span></span>|<span data-ttu-id="ab43d-170">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab43d-170">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="ab43d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab43d-171">Response</span></span>
<span data-ttu-id="ab43d-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab43d-172">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab43d-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab43d-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab43d-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab43d-174">Request</span></span>
<span data-ttu-id="ab43d-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab43d-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="ab43d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab43d-176">Response</span></span>
<span data-ttu-id="ab43d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab43d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```










