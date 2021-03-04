---
title: Obter deviceManagementConfigurationCategory
description: Leia propriedades e relações do objeto deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7b76ca23b5a89d2f8d33ebcbfd39ff3948012e6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441596"
---
# <a name="get-devicemanagementconfigurationcategory"></a><span data-ttu-id="f6239-103">Obter deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="f6239-103">Get deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="f6239-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6239-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6239-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6239-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6239-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6239-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6239-107">Leia propriedades e relações do [objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6239-107">Read properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6239-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6239-108">Prerequisites</span></span>
<span data-ttu-id="f6239-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6239-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6239-111">Permission type</span></span>|<span data-ttu-id="f6239-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6239-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6239-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6239-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6239-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6239-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6239-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6239-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6239-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6239-116">Not supported.</span></span>|
|<span data-ttu-id="f6239-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6239-117">Application</span></span>|<span data-ttu-id="f6239-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6239-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6239-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6239-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6239-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6239-120">Optional query parameters</span></span>
<span data-ttu-id="f6239-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6239-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6239-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6239-122">Request headers</span></span>
|<span data-ttu-id="f6239-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6239-123">Header</span></span>|<span data-ttu-id="f6239-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f6239-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6239-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6239-125">Authorization</span></span>|<span data-ttu-id="f6239-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6239-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6239-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6239-127">Accept</span></span>|<span data-ttu-id="f6239-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f6239-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6239-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6239-129">Request body</span></span>
<span data-ttu-id="f6239-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6239-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6239-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6239-131">Response</span></span>
<span data-ttu-id="f6239-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6239-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6239-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6239-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6239-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6239-134">Request</span></span>
<span data-ttu-id="f6239-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6239-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

### <a name="response"></a><span data-ttu-id="f6239-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6239-136">Response</span></span>
<span data-ttu-id="f6239-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6239-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "value": {
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
}
```




