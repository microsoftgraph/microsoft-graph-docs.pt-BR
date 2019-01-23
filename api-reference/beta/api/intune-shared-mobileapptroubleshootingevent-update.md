---
title: Atualizar mobileAppTroubleshootingEvent
description: Descreve o método mobileAppTroubleshootingEvent de atualização da Microsoft Graph API para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10bf103a3e796cb5a9e84f1c87ff0571c0bbf551
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429127"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="c8f8b-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c8f8b-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="c8f8b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8f8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8f8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8f8b-107">Atualize as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c8f8b-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8f8b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8f8b-108">Prerequisites</span></span>
<span data-ttu-id="c8f8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8f8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8f8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8f8b-111">Permission type</span></span>|<span data-ttu-id="c8f8b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8f8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8f8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8f8b-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c8f8b-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c8f8b-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c8f8b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f8b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8f8b-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c8f8b-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c8f8b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f8b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8f8b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8f8b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8f8b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-119">Not supported.</span></span>|
|<span data-ttu-id="c8f8b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8f8b-120">Application</span></span>|<span data-ttu-id="c8f8b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8f8b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f8b-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c8f8b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f8b-123">Request headers</span></span>
|<span data-ttu-id="c8f8b-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8f8b-124">Header</span></span>|<span data-ttu-id="c8f8b-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c8f8b-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8f8b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8f8b-126">Authorization</span></span>|<span data-ttu-id="c8f8b-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8f8b-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8f8b-128">Accept</span></span>|<span data-ttu-id="c8f8b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c8f8b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f8b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f8b-130">Request body</span></span>
<span data-ttu-id="c8f8b-131">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c8f8b-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c8f8b-132">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c8f8b-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="c8f8b-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8f8b-133">Property</span></span>|<span data-ttu-id="c8f8b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8f8b-134">Type</span></span>|<span data-ttu-id="c8f8b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8f8b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8f8b-136">id</span><span class="sxs-lookup"><span data-stu-id="c8f8b-136">id</span></span>|<span data-ttu-id="c8f8b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8f8b-137">String</span></span>|<span data-ttu-id="c8f8b-138">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-138">The GUID for the object</span></span>|
|<span data-ttu-id="c8f8b-139">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c8f8b-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="c8f8b-140">informações adicionais</span><span class="sxs-lookup"><span data-stu-id="c8f8b-140">additionalInformation</span></span>|<span data-ttu-id="c8f8b-141">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c8f8b-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c8f8b-142">Um conjunto de chave de cadeia de caracteres e pares de valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="c8f8b-143">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c8f8b-143">applicationId</span></span>|<span data-ttu-id="c8f8b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8f8b-144">String</span></span>|<span data-ttu-id="c8f8b-145">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-145">Intune application identifier.</span></span>|
|<span data-ttu-id="c8f8b-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="c8f8b-146">correlationId</span></span>|<span data-ttu-id="c8f8b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8f8b-147">String</span></span>|<span data-ttu-id="c8f8b-148">ID usado para a falha no serviço de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="c8f8b-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c8f8b-149">eventDateTime</span></span>|<span data-ttu-id="c8f8b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8f8b-150">DateTimeOffset</span></span>|<span data-ttu-id="c8f8b-151">Hora de quando o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="c8f8b-152">eventName</span><span class="sxs-lookup"><span data-stu-id="c8f8b-152">eventName</span></span>|<span data-ttu-id="c8f8b-153">String</span><span class="sxs-lookup"><span data-stu-id="c8f8b-153">String</span></span>|<span data-ttu-id="c8f8b-154">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c8f8b-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-155">Optional.</span></span>|
|<span data-ttu-id="c8f8b-156">histórico</span><span class="sxs-lookup"><span data-stu-id="c8f8b-156">history</span></span>|<span data-ttu-id="c8f8b-157">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c8f8b-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="c8f8b-158">Aplicativo Mobile Intune Item do histórico de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="c8f8b-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8f8b-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="c8f8b-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8f8b-160">String</span></span>|<span data-ttu-id="c8f8b-161">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c8f8b-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c8f8b-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c8f8b-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c8f8b-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c8f8b-164">Objeto que contém informações detalhadas sobre o erro e suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="c8f8b-165">userId</span><span class="sxs-lookup"><span data-stu-id="c8f8b-165">userId</span></span>|<span data-ttu-id="c8f8b-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8f8b-166">String</span></span>|<span data-ttu-id="c8f8b-167">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="c8f8b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f8b-168">Response</span></span>
<span data-ttu-id="c8f8b-169">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f8b-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8f8b-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8f8b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f8b-171">Request</span></span>
<span data-ttu-id="c8f8b-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="c8f8b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f8b-173">Response</span></span>
<span data-ttu-id="c8f8b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8f8b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




