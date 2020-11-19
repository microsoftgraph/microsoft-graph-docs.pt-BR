---
title: Atualizar mobileAppTroubleshootingEvent
description: Descreve o método Update mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c52a7b6cac1b4b245e7fcded390c54ca5fdf3e44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295814"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="1b525-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="1b525-103">Update mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="1b525-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b525-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b525-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1b525-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b525-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b525-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b525-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b525-108">Atualiza as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="1b525-108">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b525-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b525-109">Prerequisites</span></span>
<span data-ttu-id="1b525-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b525-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b525-112">Permission type</span></span>|<span data-ttu-id="1b525-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b525-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b525-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b525-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="1b525-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="1b525-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="1b525-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b525-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1b525-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="1b525-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="1b525-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b525-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1b525-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b525-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b525-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b525-120">Not supported.</span></span>|
|<span data-ttu-id="1b525-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b525-121">Application</span></span>||
|<span data-ttu-id="1b525-122">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="1b525-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="1b525-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b525-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1b525-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="1b525-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="1b525-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b525-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b525-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b525-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="1b525-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b525-127">Request headers</span></span>
|<span data-ttu-id="1b525-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b525-128">Header</span></span>|<span data-ttu-id="1b525-129">Valor</span><span class="sxs-lookup"><span data-stu-id="1b525-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b525-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b525-130">Authorization</span></span>|<span data-ttu-id="1b525-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b525-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b525-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b525-132">Accept</span></span>|<span data-ttu-id="1b525-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1b525-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b525-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b525-134">Request body</span></span>
<span data-ttu-id="1b525-135">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="1b525-135">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="1b525-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="1b525-136">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="1b525-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b525-137">Property</span></span>|<span data-ttu-id="1b525-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b525-138">Type</span></span>|<span data-ttu-id="1b525-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b525-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b525-140">id</span><span class="sxs-lookup"><span data-stu-id="1b525-140">id</span></span>|<span data-ttu-id="1b525-141">String</span><span class="sxs-lookup"><span data-stu-id="1b525-141">String</span></span>|<span data-ttu-id="1b525-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="1b525-142">The GUID for the object</span></span>|
|<span data-ttu-id="1b525-143">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="1b525-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="1b525-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="1b525-144">additionalInformation</span></span>|<span data-ttu-id="1b525-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1b525-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1b525-146">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="1b525-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="1b525-147">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="1b525-147">applicationId</span></span>|<span data-ttu-id="1b525-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b525-148">String</span></span>|<span data-ttu-id="1b525-149">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="1b525-149">Intune application identifier.</span></span>|
|<span data-ttu-id="1b525-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="1b525-150">correlationId</span></span>|<span data-ttu-id="1b525-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b525-151">String</span></span>|<span data-ttu-id="1b525-152">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="1b525-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="1b525-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="1b525-153">eventDateTime</span></span>|<span data-ttu-id="1b525-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b525-154">DateTimeOffset</span></span>|<span data-ttu-id="1b525-155">Hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1b525-155">Time when the event occurred.</span></span> |
|<span data-ttu-id="1b525-156">EventName</span><span class="sxs-lookup"><span data-stu-id="1b525-156">eventName</span></span>|<span data-ttu-id="1b525-157">String</span><span class="sxs-lookup"><span data-stu-id="1b525-157">String</span></span>|<span data-ttu-id="1b525-158">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="1b525-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="1b525-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1b525-159">Optional.</span></span>|
|<span data-ttu-id="1b525-160">histórico</span><span class="sxs-lookup"><span data-stu-id="1b525-160">history</span></span>|<span data-ttu-id="1b525-161">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b525-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="1b525-162">Item do histórico de solução de problemas de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="1b525-162">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="1b525-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b525-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="1b525-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b525-164">String</span></span>|<span data-ttu-id="1b525-165">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="1b525-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="1b525-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1b525-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="1b525-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1b525-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="1b525-168">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="1b525-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="1b525-169">userId</span><span class="sxs-lookup"><span data-stu-id="1b525-169">userId</span></span>|<span data-ttu-id="1b525-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b525-170">String</span></span>|<span data-ttu-id="1b525-171">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1b525-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="1b525-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b525-172">Response</span></span>
<span data-ttu-id="1b525-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b525-173">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b525-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b525-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b525-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b525-175">Request</span></span>
<span data-ttu-id="1b525-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b525-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="1b525-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b525-177">Response</span></span>
<span data-ttu-id="1b525-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b525-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```











