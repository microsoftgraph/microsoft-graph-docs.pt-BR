---
title: Atualizar mobileAppIntentAndState
description: Atualiza as propriedades de um objeto mobileAppIntentAndState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72f4a06799c04c4c06c367fedcefdec9f0341157
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707238"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="ceb1c-103">Atualizar mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="ceb1c-103">Update mobileAppIntentAndState</span></span>

<span data-ttu-id="ceb1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceb1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceb1c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceb1c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceb1c-107">Atualiza as propriedades de um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ceb1c-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb1c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceb1c-108">Prerequisites</span></span>
<span data-ttu-id="ceb1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceb1c-111">Permission type</span></span>|<span data-ttu-id="ceb1c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ceb1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb1c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceb1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb1c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb1c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ceb1c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceb1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-116">Not supported.</span></span>|
|<span data-ttu-id="ceb1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceb1c-117">Application</span></span>|<span data-ttu-id="ceb1c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb1c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceb1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ceb1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb1c-120">Request headers</span></span>
|<span data-ttu-id="ceb1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceb1c-121">Header</span></span>|<span data-ttu-id="ceb1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ceb1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceb1c-123">Authorization</span></span>|<span data-ttu-id="ceb1c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb1c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ceb1c-125">Accept</span></span>|<span data-ttu-id="ceb1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb1c-127">Request body</span></span>
<span data-ttu-id="ceb1c-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ceb1c-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="ceb1c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="ceb1c-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="ceb1c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceb1c-130">Property</span></span>|<span data-ttu-id="ceb1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceb1c-131">Type</span></span>|<span data-ttu-id="ceb1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceb1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceb1c-133">id</span><span class="sxs-lookup"><span data-stu-id="ceb1c-133">id</span></span>|<span data-ttu-id="ceb1c-134">String</span><span class="sxs-lookup"><span data-stu-id="ceb1c-134">String</span></span>|<span data-ttu-id="ceb1c-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-135">UUID for the object</span></span>|
|<span data-ttu-id="ceb1c-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ceb1c-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="ceb1c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceb1c-137">String</span></span>|<span data-ttu-id="ceb1c-138">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="ceb1c-139">userId</span><span class="sxs-lookup"><span data-stu-id="ceb1c-139">userId</span></span>|<span data-ttu-id="ceb1c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceb1c-140">String</span></span>|<span data-ttu-id="ceb1c-141">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="ceb1c-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="ceb1c-142">mobileAppList</span></span>|<span data-ttu-id="ceb1c-143">coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="ceb1c-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="ceb1c-144">A lista de efeitos e Estados de carga para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="ceb1c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb1c-145">Response</span></span>
<span data-ttu-id="ceb1c-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb1c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceb1c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceb1c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb1c-148">Request</span></span>
<span data-ttu-id="ceb1c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ceb1c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb1c-150">Response</span></span>
<span data-ttu-id="ceb1c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceb1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```





