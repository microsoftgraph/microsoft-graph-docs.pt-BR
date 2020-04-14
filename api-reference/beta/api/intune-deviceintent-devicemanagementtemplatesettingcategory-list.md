---
title: Listar deviceManagementTemplateSettingCategories
description: Listar Propriedades e relações dos objetos deviceManagementTemplateSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c5a5e9bf2ff5633b9199bff4697b5bfe7e72dec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427353"
---
# <a name="list-devicemanagementtemplatesettingcategories"></a><span data-ttu-id="adcbe-103">Listar deviceManagementTemplateSettingCategories</span><span class="sxs-lookup"><span data-stu-id="adcbe-103">List deviceManagementTemplateSettingCategories</span></span>

<span data-ttu-id="adcbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adcbe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="adcbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adcbe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="adcbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adcbe-107">Listar Propriedades e relações dos objetos [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="adcbe-107">List properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adcbe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adcbe-108">Prerequisites</span></span>
<span data-ttu-id="adcbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adcbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adcbe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adcbe-111">Permission type</span></span>|<span data-ttu-id="adcbe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adcbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adcbe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adcbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adcbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adcbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="adcbe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adcbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adcbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adcbe-116">Not supported.</span></span>|
|<span data-ttu-id="adcbe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adcbe-117">Application</span></span>|<span data-ttu-id="adcbe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adcbe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adcbe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adcbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="adcbe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adcbe-120">Request headers</span></span>
|<span data-ttu-id="adcbe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adcbe-121">Header</span></span>|<span data-ttu-id="adcbe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adcbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adcbe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adcbe-123">Authorization</span></span>|<span data-ttu-id="adcbe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adcbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adcbe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adcbe-125">Accept</span></span>|<span data-ttu-id="adcbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adcbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adcbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adcbe-127">Request body</span></span>
<span data-ttu-id="adcbe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adcbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adcbe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="adcbe-129">Response</span></span>
<span data-ttu-id="adcbe-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adcbe-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adcbe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adcbe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="adcbe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adcbe-132">Request</span></span>
<span data-ttu-id="adcbe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adcbe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
```

### <a name="response"></a><span data-ttu-id="adcbe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="adcbe-134">Response</span></span>
<span data-ttu-id="adcbe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adcbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
      "id": "cd213562-3562-cd21-6235-21cd623521cd",
      "displayName": "Display Name value",
      "hasRequiredSetting": true
    }
  ]
}
```



