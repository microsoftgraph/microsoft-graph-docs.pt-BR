---
title: Atualizar mobileAppTroubleshootingEvent
description: Descreve o método Update mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61afbd1009fed592e9ba2b0a63547d1a1d2f9ac5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694232"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="38ba7-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="38ba7-103">Update mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="38ba7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38ba7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38ba7-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38ba7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38ba7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38ba7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38ba7-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38ba7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38ba7-108">Atualiza as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="38ba7-108">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38ba7-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38ba7-109">Prerequisites</span></span>
<span data-ttu-id="38ba7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ba7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ba7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38ba7-112">Permission type</span></span>|<span data-ttu-id="38ba7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38ba7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ba7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38ba7-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="38ba7-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="38ba7-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="38ba7-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba7-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38ba7-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="38ba7-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="38ba7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38ba7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38ba7-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ba7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38ba7-120">Not supported.</span></span>|
|<span data-ttu-id="38ba7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38ba7-121">Application</span></span>||
|<span data-ttu-id="38ba7-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="38ba7-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="38ba7-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba7-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38ba7-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="38ba7-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="38ba7-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba7-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ba7-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38ba7-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="38ba7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba7-127">Request headers</span></span>
|<span data-ttu-id="38ba7-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38ba7-128">Header</span></span>|<span data-ttu-id="38ba7-129">Valor</span><span class="sxs-lookup"><span data-stu-id="38ba7-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ba7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="38ba7-130">Authorization</span></span>|<span data-ttu-id="38ba7-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38ba7-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38ba7-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38ba7-132">Accept</span></span>|<span data-ttu-id="38ba7-133">application/json</span><span class="sxs-lookup"><span data-stu-id="38ba7-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ba7-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba7-134">Request body</span></span>
<span data-ttu-id="38ba7-135">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="38ba7-135">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="38ba7-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="38ba7-136">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="38ba7-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38ba7-137">Property</span></span>|<span data-ttu-id="38ba7-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="38ba7-138">Type</span></span>|<span data-ttu-id="38ba7-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ba7-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38ba7-140">id</span><span class="sxs-lookup"><span data-stu-id="38ba7-140">id</span></span>|<span data-ttu-id="38ba7-141">String</span><span class="sxs-lookup"><span data-stu-id="38ba7-141">String</span></span>|<span data-ttu-id="38ba7-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="38ba7-142">The GUID for the object</span></span>|
|<span data-ttu-id="38ba7-143">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="38ba7-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="38ba7-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="38ba7-144">additionalInformation</span></span>|<span data-ttu-id="38ba7-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="38ba7-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="38ba7-146">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="38ba7-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="38ba7-147">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="38ba7-147">applicationId</span></span>|<span data-ttu-id="38ba7-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ba7-148">String</span></span>|<span data-ttu-id="38ba7-149">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="38ba7-149">Intune application identifier.</span></span>|
|<span data-ttu-id="38ba7-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="38ba7-150">correlationId</span></span>|<span data-ttu-id="38ba7-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ba7-151">String</span></span>|<span data-ttu-id="38ba7-152">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="38ba7-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="38ba7-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="38ba7-153">eventDateTime</span></span>|<span data-ttu-id="38ba7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ba7-154">DateTimeOffset</span></span>|<span data-ttu-id="38ba7-155">Hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="38ba7-155">Time when the event occurred.</span></span> |
|<span data-ttu-id="38ba7-156">EventName</span><span class="sxs-lookup"><span data-stu-id="38ba7-156">eventName</span></span>|<span data-ttu-id="38ba7-157">String</span><span class="sxs-lookup"><span data-stu-id="38ba7-157">String</span></span>|<span data-ttu-id="38ba7-158">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="38ba7-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="38ba7-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38ba7-159">Optional.</span></span>|
|<span data-ttu-id="38ba7-160">histórico</span><span class="sxs-lookup"><span data-stu-id="38ba7-160">history</span></span>|<span data-ttu-id="38ba7-161">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="38ba7-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="38ba7-162">Item do histórico de solução de problemas de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="38ba7-162">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="38ba7-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="38ba7-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="38ba7-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ba7-164">String</span></span>|<span data-ttu-id="38ba7-165">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="38ba7-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="38ba7-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="38ba7-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="38ba7-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="38ba7-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="38ba7-168">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="38ba7-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="38ba7-169">userId</span><span class="sxs-lookup"><span data-stu-id="38ba7-169">userId</span></span>|<span data-ttu-id="38ba7-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ba7-170">String</span></span>|<span data-ttu-id="38ba7-171">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38ba7-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="38ba7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ba7-172">Response</span></span>
<span data-ttu-id="38ba7-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38ba7-173">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ba7-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38ba7-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ba7-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba7-175">Request</span></span>
<span data-ttu-id="38ba7-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38ba7-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="38ba7-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ba7-177">Response</span></span>
<span data-ttu-id="38ba7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38ba7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












