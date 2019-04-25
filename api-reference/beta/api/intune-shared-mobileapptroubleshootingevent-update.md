---
title: Atualizar mobileAppTroubleshootingEvent
description: Descreve o método Update mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05163b0251690c990454e671ebab6aaf26fa02ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527095"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="46fee-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="46fee-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="46fee-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46fee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46fee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46fee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46fee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46fee-107">Atualiza as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="46fee-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46fee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46fee-108">Prerequisites</span></span>
<span data-ttu-id="46fee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46fee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46fee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46fee-111">Permission type</span></span>|<span data-ttu-id="46fee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46fee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46fee-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="46fee-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="46fee-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="46fee-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46fee-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="46fee-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="46fee-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="46fee-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46fee-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="46fee-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46fee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46fee-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46fee-119">Not supported.</span></span>|
|<span data-ttu-id="46fee-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46fee-120">Application</span></span>|<span data-ttu-id="46fee-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46fee-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46fee-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46fee-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="46fee-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46fee-123">Request headers</span></span>
|<span data-ttu-id="46fee-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46fee-124">Header</span></span>|<span data-ttu-id="46fee-125">Valor</span><span class="sxs-lookup"><span data-stu-id="46fee-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46fee-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="46fee-126">Authorization</span></span>|<span data-ttu-id="46fee-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46fee-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46fee-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46fee-128">Accept</span></span>|<span data-ttu-id="46fee-129">application/json</span><span class="sxs-lookup"><span data-stu-id="46fee-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46fee-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46fee-130">Request body</span></span>
<span data-ttu-id="46fee-131">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="46fee-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="46fee-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="46fee-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="46fee-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46fee-133">Property</span></span>|<span data-ttu-id="46fee-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="46fee-134">Type</span></span>|<span data-ttu-id="46fee-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="46fee-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46fee-136">id</span><span class="sxs-lookup"><span data-stu-id="46fee-136">id</span></span>|<span data-ttu-id="46fee-137">String</span><span class="sxs-lookup"><span data-stu-id="46fee-137">String</span></span>|<span data-ttu-id="46fee-138">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="46fee-138">The GUID for the object</span></span>|
|<span data-ttu-id="46fee-139">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="46fee-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="46fee-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="46fee-140">additionalInformation</span></span>|<span data-ttu-id="46fee-141">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="46fee-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="46fee-142">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="46fee-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="46fee-143">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="46fee-143">applicationId</span></span>|<span data-ttu-id="46fee-144">String</span><span class="sxs-lookup"><span data-stu-id="46fee-144">String</span></span>|<span data-ttu-id="46fee-145">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="46fee-145">Intune application identifier.</span></span>|
|<span data-ttu-id="46fee-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="46fee-146">correlationId</span></span>|<span data-ttu-id="46fee-147">String</span><span class="sxs-lookup"><span data-stu-id="46fee-147">String</span></span>|<span data-ttu-id="46fee-148">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="46fee-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="46fee-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="46fee-149">eventDateTime</span></span>|<span data-ttu-id="46fee-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46fee-150">DateTimeOffset</span></span>|<span data-ttu-id="46fee-151">Hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="46fee-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="46fee-152">EventName</span><span class="sxs-lookup"><span data-stu-id="46fee-152">eventName</span></span>|<span data-ttu-id="46fee-153">String</span><span class="sxs-lookup"><span data-stu-id="46fee-153">String</span></span>|<span data-ttu-id="46fee-154">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="46fee-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="46fee-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="46fee-155">Optional.</span></span>|
|<span data-ttu-id="46fee-156">histórico</span><span class="sxs-lookup"><span data-stu-id="46fee-156">history</span></span>|<span data-ttu-id="46fee-157">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="46fee-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="46fee-158">Item do histórico de solução de problemas de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="46fee-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="46fee-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="46fee-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="46fee-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46fee-160">String</span></span>|<span data-ttu-id="46fee-161">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="46fee-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="46fee-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="46fee-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="46fee-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="46fee-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="46fee-164">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="46fee-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="46fee-165">userId</span><span class="sxs-lookup"><span data-stu-id="46fee-165">userId</span></span>|<span data-ttu-id="46fee-166">String</span><span class="sxs-lookup"><span data-stu-id="46fee-166">String</span></span>|<span data-ttu-id="46fee-167">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46fee-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="46fee-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="46fee-168">Response</span></span>
<span data-ttu-id="46fee-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46fee-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46fee-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46fee-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="46fee-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46fee-171">Request</span></span>
<span data-ttu-id="46fee-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46fee-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="46fee-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="46fee-173">Response</span></span>
<span data-ttu-id="46fee-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46fee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




