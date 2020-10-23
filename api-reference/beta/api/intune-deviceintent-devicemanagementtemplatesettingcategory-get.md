---
title: Obter deviceManagementTemplateSettingCategory
description: Leia as propriedades e as relações do objeto deviceManagementTemplateSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a4a867d2c49031fc06c03744aa5c671fc57be78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703178"
---
# <a name="get-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="d1a8f-103">Obter deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="d1a8f-103">Get deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="d1a8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1a8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1a8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1a8f-107">Leia as propriedades e as relações do objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d1a8f-107">Read properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1a8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1a8f-108">Prerequisites</span></span>
<span data-ttu-id="d1a8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1a8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1a8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1a8f-111">Permission type</span></span>|<span data-ttu-id="d1a8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1a8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1a8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1a8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1a8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1a8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d1a8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1a8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1a8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-116">Not supported.</span></span>|
|<span data-ttu-id="d1a8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1a8f-117">Application</span></span>|<span data-ttu-id="d1a8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1a8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1a8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1a8f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1a8f-120">Optional query parameters</span></span>
<span data-ttu-id="d1a8f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1a8f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a8f-122">Request headers</span></span>
|<span data-ttu-id="d1a8f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1a8f-123">Header</span></span>|<span data-ttu-id="d1a8f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d1a8f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1a8f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1a8f-125">Authorization</span></span>|<span data-ttu-id="d1a8f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1a8f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1a8f-127">Accept</span></span>|<span data-ttu-id="d1a8f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d1a8f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1a8f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a8f-129">Request body</span></span>
<span data-ttu-id="d1a8f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1a8f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a8f-131">Response</span></span>
<span data-ttu-id="d1a8f-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-132">If successful, this method returns a `200 OK` response code and [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1a8f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1a8f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1a8f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a8f-134">Request</span></span>
<span data-ttu-id="d1a8f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="d1a8f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a8f-136">Response</span></span>
<span data-ttu-id="d1a8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1a8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
    "id": "cd213562-3562-cd21-6235-21cd623521cd",
    "displayName": "Display Name value",
    "hasRequiredSetting": true
  }
}
```





