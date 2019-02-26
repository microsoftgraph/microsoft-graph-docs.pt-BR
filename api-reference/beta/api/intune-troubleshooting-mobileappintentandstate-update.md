---
title: Atualizar mobileAppIntentAndState
description: Atualiza as propriedades de um objeto mobileAppIntentAndState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc6226237b1ebc8d080642b0cfe9bd6fd3f2b500
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173329"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="faffd-103">Atualizar mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="faffd-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="faffd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faffd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faffd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faffd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faffd-106">Atualiza as propriedades de um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="faffd-106">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faffd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="faffd-107">Prerequisites</span></span>
<span data-ttu-id="faffd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="faffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="faffd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faffd-110">Permission type</span></span>|<span data-ttu-id="faffd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="faffd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faffd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faffd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faffd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faffd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="faffd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faffd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faffd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faffd-115">Not supported.</span></span>|
|<span data-ttu-id="faffd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faffd-116">Application</span></span>|<span data-ttu-id="faffd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faffd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faffd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faffd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="faffd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faffd-119">Request headers</span></span>
|<span data-ttu-id="faffd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="faffd-120">Header</span></span>|<span data-ttu-id="faffd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="faffd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faffd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="faffd-122">Authorization</span></span>|<span data-ttu-id="faffd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faffd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faffd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="faffd-124">Accept</span></span>|<span data-ttu-id="faffd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faffd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faffd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faffd-126">Request body</span></span>
<span data-ttu-id="faffd-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="faffd-127">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="faffd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="faffd-128">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="faffd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faffd-129">Property</span></span>|<span data-ttu-id="faffd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="faffd-130">Type</span></span>|<span data-ttu-id="faffd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="faffd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faffd-132">id</span><span class="sxs-lookup"><span data-stu-id="faffd-132">id</span></span>|<span data-ttu-id="faffd-133">String</span><span class="sxs-lookup"><span data-stu-id="faffd-133">String</span></span>|<span data-ttu-id="faffd-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="faffd-134">UUID for the object</span></span>|
|<span data-ttu-id="faffd-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="faffd-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="faffd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faffd-136">String</span></span>|<span data-ttu-id="faffd-137">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="faffd-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="faffd-138">userId</span><span class="sxs-lookup"><span data-stu-id="faffd-138">userId</span></span>|<span data-ttu-id="faffd-139">String</span><span class="sxs-lookup"><span data-stu-id="faffd-139">String</span></span>|<span data-ttu-id="faffd-140">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faffd-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="faffd-141">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="faffd-141">mobileAppList</span></span>|<span data-ttu-id="faffd-142">coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="faffd-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="faffd-143">A lista de efeitos e Estados de carga para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faffd-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="faffd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="faffd-144">Response</span></span>
<span data-ttu-id="faffd-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faffd-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faffd-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faffd-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="faffd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faffd-147">Request</span></span>
<span data-ttu-id="faffd-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faffd-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faffd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="faffd-149">Response</span></span>
<span data-ttu-id="faffd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="faffd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




