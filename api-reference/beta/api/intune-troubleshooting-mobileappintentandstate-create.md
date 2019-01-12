---
title: Criar mobileAppIntentAndState
description: Crie um novo objeto de mobileAppIntentAndState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513c7ad7b6c3defdea325a1cb80161d5d554fb12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983986"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="6163c-103">Criar mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="6163c-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="6163c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6163c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6163c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6163c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6163c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6163c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6163c-107">Crie um novo objeto de [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6163c-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6163c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6163c-108">Prerequisites</span></span>
<span data-ttu-id="6163c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6163c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6163c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6163c-111">Permission type</span></span>|<span data-ttu-id="6163c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6163c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6163c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6163c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6163c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6163c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6163c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6163c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6163c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6163c-116">Not supported.</span></span>|
|<span data-ttu-id="6163c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6163c-117">Application</span></span>|<span data-ttu-id="6163c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6163c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6163c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6163c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="6163c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6163c-120">Request headers</span></span>
|<span data-ttu-id="6163c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6163c-121">Header</span></span>|<span data-ttu-id="6163c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6163c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6163c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6163c-123">Authorization</span></span>|<span data-ttu-id="6163c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6163c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6163c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6163c-125">Accept</span></span>|<span data-ttu-id="6163c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6163c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6163c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6163c-127">Request body</span></span>
<span data-ttu-id="6163c-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppIntentAndState.</span><span class="sxs-lookup"><span data-stu-id="6163c-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="6163c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppIntentAndState.</span><span class="sxs-lookup"><span data-stu-id="6163c-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="6163c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6163c-130">Property</span></span>|<span data-ttu-id="6163c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6163c-131">Type</span></span>|<span data-ttu-id="6163c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6163c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6163c-133">id</span><span class="sxs-lookup"><span data-stu-id="6163c-133">id</span></span>|<span data-ttu-id="6163c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6163c-134">String</span></span>|<span data-ttu-id="6163c-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6163c-135">UUID for the object</span></span>|
|<span data-ttu-id="6163c-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6163c-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="6163c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6163c-137">String</span></span>|<span data-ttu-id="6163c-138">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="6163c-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="6163c-139">userId</span><span class="sxs-lookup"><span data-stu-id="6163c-139">userId</span></span>|<span data-ttu-id="6163c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6163c-140">String</span></span>|<span data-ttu-id="6163c-141">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6163c-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="6163c-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="6163c-142">mobileAppList</span></span>|<span data-ttu-id="6163c-143">coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="6163c-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="6163c-144">A lista de propósitos de carga e estados do inquilino.</span><span class="sxs-lookup"><span data-stu-id="6163c-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="6163c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6163c-145">Response</span></span>
<span data-ttu-id="6163c-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6163c-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6163c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6163c-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="6163c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6163c-148">Request</span></span>
<span data-ttu-id="6163c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6163c-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
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

### <a name="response"></a><span data-ttu-id="6163c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6163c-150">Response</span></span>
<span data-ttu-id="6163c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6163c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





