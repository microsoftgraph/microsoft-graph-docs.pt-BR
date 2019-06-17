---
title: Listar deviceManagementTemplateSettingCategories
description: Listar Propriedades e relações dos objetos deviceManagementTemplateSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6829cc41efec17f038a01eab685b01e24d0004be
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959618"
---
# <a name="list-devicemanagementtemplatesettingcategories"></a><span data-ttu-id="03729-103">Listar deviceManagementTemplateSettingCategories</span><span class="sxs-lookup"><span data-stu-id="03729-103">List deviceManagementTemplateSettingCategories</span></span>

> <span data-ttu-id="03729-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03729-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03729-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03729-106">Listar Propriedades e relações dos objetos [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="03729-106">List properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03729-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03729-107">Prerequisites</span></span>
<span data-ttu-id="03729-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03729-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03729-110">Permission type</span></span>|<span data-ttu-id="03729-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03729-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03729-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03729-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03729-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03729-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03729-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03729-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03729-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03729-115">Not supported.</span></span>|
|<span data-ttu-id="03729-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03729-116">Application</span></span>|<span data-ttu-id="03729-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03729-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03729-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03729-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="03729-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03729-119">Request headers</span></span>
|<span data-ttu-id="03729-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03729-120">Header</span></span>|<span data-ttu-id="03729-121">Valor</span><span class="sxs-lookup"><span data-stu-id="03729-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03729-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="03729-122">Authorization</span></span>|<span data-ttu-id="03729-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03729-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03729-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03729-124">Accept</span></span>|<span data-ttu-id="03729-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03729-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03729-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03729-126">Request body</span></span>
<span data-ttu-id="03729-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03729-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03729-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="03729-128">Response</span></span>
<span data-ttu-id="03729-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03729-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03729-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03729-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="03729-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03729-131">Request</span></span>
<span data-ttu-id="03729-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03729-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
```

### <a name="response"></a><span data-ttu-id="03729-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="03729-133">Response</span></span>
<span data-ttu-id="03729-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03729-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
      "id": "cd213562-3562-cd21-6235-21cd623521cd",
      "displayName": "Display Name value"
    }
  ]
}
```





