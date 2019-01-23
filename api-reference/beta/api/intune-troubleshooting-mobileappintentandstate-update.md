---
title: Atualizar mobileAppIntentAndState
description: Atualize as propriedades de um objeto mobileAppIntentAndState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7157711819e4a5b3d4fbeb6ea6c8fce136da9380
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405188"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="cca46-103">Atualizar mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="cca46-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="cca46-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cca46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cca46-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cca46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cca46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cca46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cca46-107">Atualize as propriedades de um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="cca46-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cca46-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cca46-108">Prerequisites</span></span>
<span data-ttu-id="cca46-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cca46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cca46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cca46-111">Permission type</span></span>|<span data-ttu-id="cca46-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cca46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cca46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cca46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cca46-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca46-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cca46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cca46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cca46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca46-116">Not supported.</span></span>|
|<span data-ttu-id="cca46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cca46-117">Application</span></span>|<span data-ttu-id="cca46-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cca46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cca46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cca46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cca46-120">Request headers</span></span>
|<span data-ttu-id="cca46-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cca46-121">Header</span></span>|<span data-ttu-id="cca46-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cca46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cca46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cca46-123">Authorization</span></span>|<span data-ttu-id="cca46-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cca46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cca46-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cca46-125">Accept</span></span>|<span data-ttu-id="cca46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cca46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cca46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cca46-127">Request body</span></span>
<span data-ttu-id="cca46-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="cca46-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="cca46-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="cca46-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="cca46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cca46-130">Property</span></span>|<span data-ttu-id="cca46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cca46-131">Type</span></span>|<span data-ttu-id="cca46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cca46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cca46-133">id</span><span class="sxs-lookup"><span data-stu-id="cca46-133">id</span></span>|<span data-ttu-id="cca46-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cca46-134">String</span></span>|<span data-ttu-id="cca46-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="cca46-135">UUID for the object</span></span>|
|<span data-ttu-id="cca46-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cca46-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="cca46-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cca46-137">String</span></span>|<span data-ttu-id="cca46-138">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="cca46-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="cca46-139">userId</span><span class="sxs-lookup"><span data-stu-id="cca46-139">userId</span></span>|<span data-ttu-id="cca46-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cca46-140">String</span></span>|<span data-ttu-id="cca46-141">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cca46-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="cca46-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="cca46-142">mobileAppList</span></span>|<span data-ttu-id="cca46-143">coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="cca46-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="cca46-144">A lista de propósitos de carga e estados do inquilino.</span><span class="sxs-lookup"><span data-stu-id="cca46-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="cca46-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca46-145">Response</span></span>
<span data-ttu-id="cca46-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cca46-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca46-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cca46-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="cca46-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cca46-148">Request</span></span>
<span data-ttu-id="cca46-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cca46-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cca46-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca46-150">Response</span></span>
<span data-ttu-id="cca46-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cca46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




