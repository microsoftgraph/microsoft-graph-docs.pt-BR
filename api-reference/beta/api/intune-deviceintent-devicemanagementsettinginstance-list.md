---
title: Listar deviceManagementSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45bff5b1a04dab1b4c37ef76f10388ae48e3f71e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300168"
---
# <a name="list-devicemanagementsettinginstances"></a><span data-ttu-id="9b610-103">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="9b610-103">List deviceManagementSettingInstances</span></span>

<span data-ttu-id="9b610-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b610-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b610-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b610-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b610-107">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="9b610-107">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b610-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b610-108">Prerequisites</span></span>
<span data-ttu-id="9b610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b610-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b610-111">Permission type</span></span>|<span data-ttu-id="9b610-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b610-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b610-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b610-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b610-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b610-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b610-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b610-116">Not supported.</span></span>|
|<span data-ttu-id="9b610-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b610-117">Application</span></span>|<span data-ttu-id="9b610-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b610-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b610-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b610-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9b610-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b610-120">Request headers</span></span>
|<span data-ttu-id="9b610-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b610-121">Header</span></span>|<span data-ttu-id="9b610-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b610-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b610-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b610-123">Authorization</span></span>|<span data-ttu-id="9b610-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b610-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b610-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b610-125">Accept</span></span>|<span data-ttu-id="9b610-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b610-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b610-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b610-127">Request body</span></span>
<span data-ttu-id="9b610-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b610-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b610-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b610-129">Response</span></span>
<span data-ttu-id="9b610-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b610-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b610-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b610-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b610-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b610-132">Request</span></span>
<span data-ttu-id="9b610-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b610-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="9b610-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b610-134">Response</span></span>
<span data-ttu-id="9b610-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b610-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```




