---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método Create mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 271e5b9b88608a89cf6ec0df9f4d7376757ba6c2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694281"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="0641d-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="0641d-103">Create mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="0641d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0641d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0641d-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0641d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0641d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0641d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0641d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0641d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0641d-108">Criar um novo objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0641d-108">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0641d-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0641d-109">Prerequisites</span></span>
<span data-ttu-id="0641d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0641d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0641d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0641d-112">Permission type</span></span>|<span data-ttu-id="0641d-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0641d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0641d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0641d-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="0641d-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0641d-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="0641d-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0641d-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="0641d-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="0641d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0641d-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0641d-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0641d-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0641d-120">Not supported.</span></span>|
|<span data-ttu-id="0641d-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0641d-121">Application</span></span>||
|<span data-ttu-id="0641d-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0641d-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="0641d-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0641d-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="0641d-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="0641d-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0641d-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0641d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0641d-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0641d-127">Request headers</span></span>
|<span data-ttu-id="0641d-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0641d-128">Header</span></span>|<span data-ttu-id="0641d-129">Valor</span><span class="sxs-lookup"><span data-stu-id="0641d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0641d-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="0641d-130">Authorization</span></span>|<span data-ttu-id="0641d-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0641d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0641d-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0641d-132">Accept</span></span>|<span data-ttu-id="0641d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0641d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0641d-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0641d-134">Request body</span></span>
<span data-ttu-id="0641d-135">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="0641d-135">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="0641d-136">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="0641d-136">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="0641d-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0641d-137">Property</span></span>|<span data-ttu-id="0641d-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0641d-138">Type</span></span>|<span data-ttu-id="0641d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0641d-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0641d-140">id</span><span class="sxs-lookup"><span data-stu-id="0641d-140">id</span></span>|<span data-ttu-id="0641d-141">String</span><span class="sxs-lookup"><span data-stu-id="0641d-141">String</span></span>|<span data-ttu-id="0641d-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="0641d-142">The GUID for the object</span></span>|
|<span data-ttu-id="0641d-143">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="0641d-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="0641d-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="0641d-144">additionalInformation</span></span>|<span data-ttu-id="0641d-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0641d-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0641d-146">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="0641d-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="0641d-147">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="0641d-147">applicationId</span></span>|<span data-ttu-id="0641d-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0641d-148">String</span></span>|<span data-ttu-id="0641d-149">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="0641d-149">Intune application identifier.</span></span>|
|<span data-ttu-id="0641d-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="0641d-150">correlationId</span></span>|<span data-ttu-id="0641d-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0641d-151">String</span></span>|<span data-ttu-id="0641d-152">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="0641d-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="0641d-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0641d-153">eventDateTime</span></span>|<span data-ttu-id="0641d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0641d-154">DateTimeOffset</span></span>|<span data-ttu-id="0641d-155">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0641d-155">Time when the event occurred .</span></span> |
|<span data-ttu-id="0641d-156">EventName</span><span class="sxs-lookup"><span data-stu-id="0641d-156">eventName</span></span>|<span data-ttu-id="0641d-157">String</span><span class="sxs-lookup"><span data-stu-id="0641d-157">String</span></span>|<span data-ttu-id="0641d-158">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="0641d-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="0641d-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0641d-159">Optional.</span></span>|
|<span data-ttu-id="0641d-160">histórico</span><span class="sxs-lookup"><span data-stu-id="0641d-160">history</span></span>|<span data-ttu-id="0641d-161">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0641d-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="0641d-162">Item do histórico de solução de problemas do aplicativo móvel do Intune</span><span class="sxs-lookup"><span data-stu-id="0641d-162">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="0641d-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0641d-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="0641d-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0641d-164">String</span></span>|<span data-ttu-id="0641d-165">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="0641d-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="0641d-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0641d-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="0641d-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0641d-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="0641d-168">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="0641d-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="0641d-169">userId</span><span class="sxs-lookup"><span data-stu-id="0641d-169">userId</span></span>|<span data-ttu-id="0641d-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0641d-170">String</span></span>|<span data-ttu-id="0641d-171">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0641d-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="0641d-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="0641d-172">Response</span></span>
<span data-ttu-id="0641d-173">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0641d-173">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0641d-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0641d-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="0641d-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0641d-175">Request</span></span>
<span data-ttu-id="0641d-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0641d-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="0641d-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="0641d-177">Response</span></span>
<span data-ttu-id="0641d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0641d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












