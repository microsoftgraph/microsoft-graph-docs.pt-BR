---
title: Listar deviceManagementStringSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementStringSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d061921c02bcd7a6137bad07ee38e36c7122a1f3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959863"
---
# <a name="list-devicemanagementstringsettinginstances"></a><span data-ttu-id="d2626-103">Listar deviceManagementStringSettingInstances</span><span class="sxs-lookup"><span data-stu-id="d2626-103">List deviceManagementStringSettingInstances</span></span>

> <span data-ttu-id="d2626-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2626-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2626-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2626-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2626-106">Listar Propriedades e relações dos objetos [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="d2626-106">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2626-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2626-107">Prerequisites</span></span>
<span data-ttu-id="d2626-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2626-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2626-110">Permission type</span></span>|<span data-ttu-id="d2626-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2626-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2626-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2626-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2626-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2626-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d2626-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2626-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2626-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2626-115">Not supported.</span></span>|
|<span data-ttu-id="d2626-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2626-116">Application</span></span>|<span data-ttu-id="d2626-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2626-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2626-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2626-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="d2626-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2626-119">Request headers</span></span>
|<span data-ttu-id="d2626-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2626-120">Header</span></span>|<span data-ttu-id="d2626-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d2626-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2626-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2626-122">Authorization</span></span>|<span data-ttu-id="d2626-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2626-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2626-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2626-124">Accept</span></span>|<span data-ttu-id="d2626-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2626-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2626-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2626-126">Request body</span></span>
<span data-ttu-id="d2626-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2626-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2626-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2626-128">Response</span></span>
<span data-ttu-id="d2626-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2626-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2626-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2626-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2626-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2626-131">Request</span></span>
<span data-ttu-id="d2626-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2626-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="d2626-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2626-133">Response</span></span>
<span data-ttu-id="d2626-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2626-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
      "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": "Value value"
    }
  ]
}
```





