---
title: Listar deviceManagementConfigurationCategories
description: Listar propriedades e relações dos objetos deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3282f9e3d98865cc01e99fe2a171b1dfc36e9136
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441582"
---
# <a name="list-devicemanagementconfigurationcategories"></a><span data-ttu-id="b41e6-103">Listar deviceManagementConfigurationCategories</span><span class="sxs-lookup"><span data-stu-id="b41e6-103">List deviceManagementConfigurationCategories</span></span>

<span data-ttu-id="b41e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b41e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b41e6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b41e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b41e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b41e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b41e6-107">Listar propriedades e relações dos [objetos deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b41e6-107">List properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b41e6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b41e6-108">Prerequisites</span></span>
<span data-ttu-id="b41e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b41e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b41e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b41e6-111">Permission type</span></span>|<span data-ttu-id="b41e6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b41e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b41e6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b41e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b41e6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b41e6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b41e6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b41e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b41e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b41e6-116">Not supported.</span></span>|
|<span data-ttu-id="b41e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b41e6-117">Application</span></span>|<span data-ttu-id="b41e6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b41e6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b41e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b41e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="b41e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b41e6-120">Request headers</span></span>
|<span data-ttu-id="b41e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b41e6-121">Header</span></span>|<span data-ttu-id="b41e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b41e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b41e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b41e6-123">Authorization</span></span>|<span data-ttu-id="b41e6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b41e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b41e6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b41e6-125">Accept</span></span>|<span data-ttu-id="b41e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b41e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b41e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b41e6-127">Request body</span></span>
<span data-ttu-id="b41e6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b41e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b41e6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41e6-129">Response</span></span>
<span data-ttu-id="b41e6-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b41e6-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b41e6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b41e6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b41e6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b41e6-132">Request</span></span>
<span data-ttu-id="b41e6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b41e6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationCategories
```

### <a name="response"></a><span data-ttu-id="b41e6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41e6-134">Response</span></span>
<span data-ttu-id="b41e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b41e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 603

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
      "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "platforms": "macOS",
      "technologies": "mdm",
      "settingUsage": "configuration",
      "parentCategoryId": "Parent Category Id value",
      "rootCategoryId": "Root Category Id value",
      "childCategoryIds": [
        "Child Category Ids value"
      ]
    }
  ]
}
```




